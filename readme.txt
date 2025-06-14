clusters
    staging
        flux-system
            gotk-sync.yaml <-- points to clusters/staging
            apps.yaml in clusters/staging <-- includes to apps/staging, refers to flux-system namespace
            kustomization.yaml in apps/staging <-- creates namespaace for linkding, points to resource for ../../base/linkding
            deployment.yaml, namespace.yaml <-- actual container config/namespace where it will live
            
